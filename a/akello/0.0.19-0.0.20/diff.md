# Comparing `tmp/akello-0.0.19.tar.gz` & `tmp/akello-0.0.20.tar.gz`

## Comparing `akello-0.0.19.tar` & `akello-0.0.20.tar`

### file list

```diff
@@ -1,85 +1,120 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.19/Dockerfile
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 akello-0.0.19/Dockerfile.aws.lambda
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/__init__.py
--rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.19/openapi.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.19/openapi.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.19/publish_test_pypi.sh
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 akello-0.0.19/requirements.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 akello-0.0.19/akello/__init__.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 akello-0.0.19/akello/main.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 akello-0.0.19/akello/management.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.19/akello/secrets.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.19/akello/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/__init__.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/endpoints/__init__.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/endpoints/financial_model.py
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/endpoints/registry.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/endpoints/reports.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 akello-0.0.19/akello/api/v1/endpoints/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/auth/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.19/akello/auth/provider.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.19/akello/auth/aws_cognito/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/auth/aws_cognito/__init__.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 akello-0.0.19/akello/auth/aws_cognito/auth_settings.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 akello-0.0.19/akello/auth/aws_cognito/aws_cognito.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.19/akello/commands/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/commands/__init__.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 akello-0.0.19/akello/commands/generate_mock_demo_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/decorators/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 akello-0.0.19/akello/decorators/mixin.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/README.md
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/__init__.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/query.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/models/__init__.py
--rw-r--r--   0        0        0    20032 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/models/financial_model.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/models/questionnaire.py
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/models/registry.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 akello-0.0.19/akello/dynamodb/models/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/fhir/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.19/akello/fhir/hl7/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.19/akello/fhir/hl7/__init__.py
--rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.19/akello/fhir/hl7/fhir_v6_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/mixin_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/aws_ses/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/aws_ses/email.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/metriport/README.md
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/metriport/__init__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/metriport/api.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/metriport/webhook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/metriport/tests/__init__.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 akello-0.0.19/akello/plugins/metriport/tests/test_metriport.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/R4/__init__.py
--rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/R4/gad7.R4.json
--rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/R4/phq9.R4.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/custom/FHIR_weights.yaml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/custom/api_weights.yaml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/questionnaires/gad7.json
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.19/akello/screeners/questionnaires/phq9.json
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/__init__.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/admin.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/decorators.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/patient.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/registry.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/registry_membership.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/reports.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/screeners.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/user.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_admin_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_decorators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_patient_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_registry_membership.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_registry_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_reports_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_screeners_service.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 akello-0.0.19/akello/services/tests/test_user_service.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 akello-0.0.19/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.19/LICENSE
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 akello-0.0.19/README.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 akello-0.0.19/pyproject.toml
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 akello-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.20/.dockerignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.20/Dockerfile
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.20/Dockerfile.aws.lambda
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/__init__.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.20/management.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/module_name.md
+-rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.20/openapi.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.20/openapi.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.20/publish_test_pypi.sh
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 akello-0.0.20/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/.gitignore
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/api-server.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/modules.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/vcs.xml
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/workspace.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 akello-0.0.20/akello/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.20/akello/app_configs.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.20/akello/main.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.20/akello/secrets.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.20/akello/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/registry.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/reports.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/provider.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/__init__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/auth_settings.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/aws_cognito.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/__init__.py
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/models.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/connector/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/connector/dynamodb.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/connector/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/decorators/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.20/akello/decorators/akello_plan_tier.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.20/akello/decorators/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/__init__.py
+-rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/fhir.schema.json
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/hl7/README.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/hl7/__init__.py
+-rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/hl7/fhir_v6_models.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/__init__.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/FHIR/phq9_fhir.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/FHIR/phq9_response.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/R4/__init__.py
+-rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/R4/gad7.R4.json
+-rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/R4/phq9.R4.json
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/FHIR_weights.template
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/api_weights.template
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_GAD-7.yaml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_HEADS-ED.yaml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_PHQ-9.yaml
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_PMQ.yaml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/questionnaires/gad7.json
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/questionnaires/phq9.json
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/__init__.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/akello_apps.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/registry.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/reports.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/screeners.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/stripe_payment.py
+-rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/user.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_decorators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_registry_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_reports_service.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_screeners_service.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/utils/email.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.20/commands/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/commands/__init__.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/__init__.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/patient.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/registry.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/treatment_log.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/user.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.20/docs/Makefile
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.fhir.rst
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.fhir.v1.endpoints.rst
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.fhir.v1.rst
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.rst
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.auth.aws_cognito.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.auth.rst
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.db.connector.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.db.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.decorators.rst
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.fhir.hl7.rst
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.fhir.rst
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.screeners.R4.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.screeners.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.services.rst
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.services.tests.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.utils.rst
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.20/docs/conf.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.20/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.20/docs/make.bat
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.20/docs/modules.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/README.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/generate_data.sh
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/load_fhir_data.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.20/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.20/LICENSE
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.20/README.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 akello-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 akello-0.0.20/PKG-INFO
```

### Comparing `akello-0.0.19/openapi.json` & `akello-0.0.20/openapi.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/requirements.txt` & `akello-0.0.20/requirements.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,135 @@
 aiofile==3.8.8
-aiohttp==3.8.5
+aiofiles==23.2.1
+aiohttp==3.9.2
 aiosignal==1.3.1
+alabaster==0.7.16
 annotated-types==0.5.0
 anyio==3.7.1
 async-lru==2.0.4
 async-timeout==4.0.3
 attrs==23.1.0
 aws-cdk-lib==2.103.1
 aws-cdk.asset-awscli-v1==2.2.201
 aws-cdk.asset-kubectl-v20==2.1.2
 aws-cdk.asset-node-proxy-agent-v6==2.0.1
 aws-cdk.aws-codestar-alpha==2.103.1a0
 aws-lambda-powertools==2.26.0
+Babel==2.14.0
+beautifulsoup4==4.12.3
 boto3==1.28.57
 botocore==1.31.57
+bs4==0.0.2
 build==1.0.3
 caio==0.9.13
 cattrs==23.1.2
 certifi==2023.7.22
 cffi==1.16.0
 charset-normalizer==3.3.0
 click==8.1.7
 cognitojwt==1.4.1
+commonmark==0.9.1
 constructs==10.3.0
-cryptography==42.0.2
+cryptography==42.0.4
 dnspython==2.4.2
 docutils==0.20.1
 ecdsa==0.18.0
 email-validator==2.0.0.post2
 exceptiongroup==1.1.3
+Faker==22.6.0
 fastapi==0.109.1
 fastapi-cognito==2.4.2
+fhir.resources==7.1.0
+flatten-json==0.1.14
 frozenlist==1.4.0
 h11==0.14.0
 httpcore==0.18.0
 httptools==0.6.0
 httpx==0.25.0
 idna==3.4
+imagesize==1.4.1
 importlib-metadata==6.8.0
 importlib-resources==6.1.0
 install==1.3.5
 itsdangerous==2.1.2
 jaraco.classes==3.3.0
 Jinja2==3.1.3
 jmespath==1.0.1
 jsii==1.91.0
+jsonmerge==1.9.2
+jsonpath-ng==1.6.1
+jsonschema==4.21.1
+jsonschema-specifications==2023.12.1
 keyring==24.2.0
 mangum==0.17.0
+Markdown==3.6
 markdown-it-py==3.0.0
 MarkupSafe==2.1.3
 mdurl==0.1.2
-# metriport==8.0.0a1
 more-itertools==10.1.0
 multidict==6.0.4
 nh3==0.2.14
-orjson==3.9.7
+numpy==1.26.4
+orjson==3.9.15
 packaging==23.2
-pkginfo==1.9.6
+pandas==2.2.1
+ply==3.11
 publication==0.0.3
 pyasn1==0.5.0
 pycparser==2.21
 pydantic==2.4.2
 pydantic-extra-types==2.1.0
 pydantic-settings==2.0.3
+pydantic-to-typescript==1.0.10
 pydantic_core==2.10.1
 Pygments==2.16.1
 pyngrok==7.0.5
 pyproject_hooks==1.0.0
 python-dateutil==2.8.2
 python-dotenv==1.0.0
+python-http-client==3.3.7
 python-jose==3.3.0
 python-multipart==0.0.7
+pytz==2024.1
 PyYAML==6.0.1
 readme-renderer==42.0
+recommonmark==0.7.1
+referencing==0.33.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.6.0
+rpds-py==0.18.0
 rsa==4.9
 s3transfer==0.7.0
+sendgrid==6.11.0
 six==1.16.0
 sniffio==1.3.0
-starlette==0.36.2
-twine==4.0.2
+snowballstemmer==2.2.0
+soupsieve==2.5
+Sphinx==7.2.6
+sphinx-markdown-builder==0.6.6
+sphinx-markdown-tables==0.0.17
+sphinx-md==0.0.4
+sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-jsmath==1.0.1
+sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-serializinghtml==1.1.10
+starkbank-ecdsa==2.2.0
+starlette==0.35.1
+stripe==8.8.0
+tabulate==0.9.0
 typeguard==2.13.3
+typer==0.9.0
 typing_extensions==4.8.0
+tzdata==2024.1
+ua-parser==0.18.0
 ujson==5.8.0
 urllib3==1.26.18
+user-agents==2.2.0
 uvicorn==0.23.2
-uvloop==0.17.0
 watchfiles==0.20.0
 websockets==11.0.3
 yarl==1.9.2
 zipp==3.17.0
```

### Comparing `akello-0.0.19/akello/main.py` & `akello-0.0.20/akello/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, sys
 from fastapi import FastAPI
 from akello.settings import *
-from akello.api.v1.api import router as api_router
+from akello.api.app.v1.api import router as api_router
+#from akello_apps.metriport.webhooks.metriport_webhook import router as metriport_webhook
+#from akello_apps.typeform.webhooks.typeform_webhook import router as typeform_webhook
 from fastapi.middleware.cors import CORSMiddleware
-from akello.plugins.metriport.webhook import router as metriport_webhook
-from akello.plugins.metriport import MetriportMixinStartFHIRConsolidatedQuery
 from mangum import Mangum
 from aws_lambda_powertools import Logger
 from pydantic_settings import BaseSettings
 
 logger = Logger(service="mangum")
 
 
@@ -20,14 +20,15 @@
 
 settings = Settings()
 
 def init_webhooks(base_url):
     # Update inbound traffic via APIs to use the public-facing ngrok URL
     pass
 
+
 if settings.USE_NGROK and os.environ.get("NGROK_AUTHTOKEN"):
     # pyngrok should only ever be installed or initialized in a dev environment when this flag is set
     from pyngrok import ngrok
 
     # Get the dev server port (defaults to 8000 for Uvicorn, can be overridden with `--port`
     # when starting the server
     port = sys.argv[sys.argv.index("--port") + 1] if "--port" in sys.argv else "8000"
@@ -53,33 +54,20 @@
 @app.get("/")
 def root():
     return {"message": "api.akello.io"}
 
 
 app.include_router(api_router, prefix="/v1")
 
-app.state.after_patient_referral_mixins = []
-app.state.before_patient_session_mixins = []
-app.state.fetch_patient_fhir_data_mixin = None  # fetch from stored FHIR Server
-app.state.fetch_patient_fhir_data_hie_mixin = None  # fetch across HIEs
-app.state.sms_plugin = None
-app.state.email_plugin = None
-app.state.patient_form_plugin = None
-
-
-"""
-TODO: Should be implemented by apps that extend the base server
-
-metriport_api_key = os.getenv('METRIPORT_API_KEY', None)
-metriport_api_url = os.getenv('METRIPORT_API_URL', None)
-if metriport_api_key != '$METRIPORT_API_KEY' and metriport_api_url != '$METRIPORT_API_URL' and metriport_api_key and metriport_api_url:    
-    #app.state.after_patient_referral_mixins.append(MetriportMixinStartFHIRConsolidatedQuery)
-    app.state.fetch_patient_fhir_data_mixin = MetriportMixinStartFHIRConsolidatedQuery
-    app.include_router(metriport_webhook, prefix="/v1/integrations", tags=["Integrations"])
-"""
+#TODO: Should be implemented by apps that extend the base server
+#metriport_api_key = os.getenv('METRIPORT_API_KEY', None)
+#metriport_api_url = os.getenv('METRIPORT_API_URL', None)
+#if metriport_api_key != '$METRIPORT_API_KEY' and metriport_api_url != '$METRIPORT_API_URL' and metriport_api_key and metriport_api_url:
+#app.include_router(metriport_webhook, prefix="/v1/integrations/metriport", tags=["Integrations"])
+#app.include_router(typeform_webhook, prefix="/v1/integrations/typeform", tags=["Integrations"])
 
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
```

### Comparing `akello-0.0.19/akello/secrets.py` & `akello-0.0.20/akello/secrets.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/api/v1/endpoints/reports.py` & `akello-0.0.20/akello/api/app/v1/endpoints/reports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 from fastapi import APIRouter, Depends
 from akello.services.user import  UserService
 from akello.auth.provider import auth_token_check
 from akello.auth.aws_cognito.auth_settings import CognitoTokenCustom
 from akello.services.reports import ReportsService
-
+from akello.decorators.akello_plan_tier import akello_plan_check
+from akello.db.types import AkelloPlanTier
 
 logger = logging.getLogger('mangum')
 router = APIRouter()
 
 @router.get("/{registry_id}/billing")
+@akello_plan_check(tiers=[AkelloPlanTier.individual, AkelloPlanTier.teams, AkelloPlanTier.enterprise])
 async def billing_report_monthly(registry_id: str, from_date: int, to_date: int, auth: CognitoTokenCustom = Depends(auth_token_check)):
     UserService.check_registry_access(auth.cognito_id, registry_id)
     data = ReportsService.get_billing_report(registry_id, from_date, to_date)
     return data
 
 @router.get("/{registry_id}/dashboard-stats")
 async def get_registry_stats(registry_id: str, from_date: int, to_date: int, auth: CognitoTokenCustom = Depends(auth_token_check)):
```

### Comparing `akello-0.0.19/akello/auth/aws_cognito/README.md` & `akello-0.0.20/akello/auth/aws_cognito/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/auth/aws_cognito/auth_settings.py` & `akello-0.0.20/akello/auth/aws_cognito/auth_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,7 +33,9 @@
     iss: HttpUrl
     exp: int
     iat: int
     jti: str
     client_id: Optional[str] = None
     username: Optional[str] = None
     email: str
+    family_name: Optional[str] = None
+    given_name: Optional[str] = None
```

### Comparing `akello-0.0.19/akello/auth/aws_cognito/aws_cognito.py` & `akello-0.0.20/akello/auth/aws_cognito/aws_cognito.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from fastapi import Request, HTTPException
 from pydantic_settings import BaseSettings
 from pydantic.types import Any
 from typing import Optional
 from fastapi_cognito import CognitoAuth, CognitoSettings
+from akello.auth.aws_cognito.auth_settings import CognitoTokenCustom
+
 from pydantic import BaseModel, HttpUrl, Field,parse_obj_as
 from jose import jwt
 
 
 AWS_COGNITO_APP_CLIENT_ID = os.getenv('AWS_COGNITO_APP_CLIENT_ID')
 AWS_COGNITO_USERPOOL_ID = os.getenv('AWS_COGNITO_USERPOOL_ID')
 AKELLO_COGNITO_URL = os.getenv('AKELLO_COGNITO_URL')
@@ -25,36 +27,19 @@
             "userpool_id": AWS_COGNITO_USERPOOL_ID,
             "app_client_id": AWS_COGNITO_APP_CLIENT_ID,
             **({"endpoint": AKELLO_COGNITO_URL} if os.environ.get('AKELLO_COGNITO_URL') else {})
         },
     }
 
 
-class CognitoTokenCustom(BaseModel):
-    origin_jti: Optional[str] = None
-    cognito_id: str = Field(alias="sub")
-    event_id: Optional[str] = None
-    token_use: str
-    scope: Optional[str] = None
-    auth_time: int
-    iss: HttpUrl
-    exp: int
-    iat: int
-    jti: str
-    client_id: Optional[str] = None
-    username: Optional[str] = None
-    # email: str - pull this from the user attributes
-    sub: str
-
-
 async def local_auth_required(request: Request) -> CognitoTokenCustom:
     try:        
         auth_token = request.headers.get('Authorization').replace('Bearer ', '')        
         decoded_token = jwt.get_unverified_claims(auth_token) #NOSONAR
-        decoded_token["email"] = decoded_token["username"]
+        decoded_token["email"] = decoded_token["username"]        
     except Exception as e:
         print(e)
         raise HTTPException(status_code=401, detail="Unauthroized")
     return parse_obj_as(CognitoTokenCustom, decoded_token)
 
 auth_provider = CognitoAuth(
     settings=CognitoSettings.from_global_settings(Settings()), userpool_name="us",
```

### Comparing `akello-0.0.19/akello/dynamodb/models/registry.py` & `akello-0.0.20/akello/db/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,118 @@
-from akello.dynamodb.models import RegistryDBBaseModel
+from decimal import Decimal
+import datetime, json
 from enum import Enum
+from typing import List, Optional, Union
+
+from boto3.dynamodb.conditions import Key
+from botocore.exceptions import ClientError
 from pydantic import BaseModel
-from typing import List, Optional
-import json
-import datetime
 
+from akello.db.connector.dynamodb import registry_db, RegistryDBBaseModel
+
+
+class UserMembershipType(str, Enum):
+    account = 'account'
+    organization = 'organization'
+
+class QuestionResponse(BaseModel):
+    id: str
+    response: str
+    score: int
+
+
+class Question(BaseModel):
+    id: str
+    question: str
+    responses: List[QuestionResponse]
+    score: int = 0
+
+
+class FHIRWeight(BaseModel):
+    name: str
+    jsonPath: str
+    codes: List[str]
+    weight: int
+
+
+class Measurement(BaseModel):
+    name: str
+    uid: str
+    type: str
+    active: Optional[bool] = False
+    measurements: Union[List[Question], List[FHIRWeight]]
+
+
+class AkelloPlanTier(str, Enum):
+    free = 'Free'
+    individual = 'Individual'
+    teams = 'Teams'
+    enterprise = 'Enterprise'
+
+class UserRole(str, Enum):
+    care_manager = 'Care Manager'
+    primary_care_physician = 'Primary Care Physician'
+    consulting_psychiatrist = 'Consulting Psychiatrist'
+    clinical_ops = 'Clinical Ops'
+    finance = 'Finance'
+
+
+class UserInvite(BaseModel):
+    email: str
+    first_name: str
+    last_name: str
+    invited_by: str
+    registry_id: str
+    date_created: int
+    role: UserRole
+
+    @property
+    def partition_key(self) -> str:
+        return 'invite:' + self.email
+
+    @property
+    def sort_key(self) -> str:
+        return 'registry:' + self.registry_id
+
+    @staticmethod
+    def create(cognito_user_id, email, role: UserRole, registry_id):
+        response = registry_db.put_item(
+            Item={
+                "partition_key": 'invite:%s' % email,
+                "sort_key": registry_id,
+                "invited_by": cognito_user_id,
+                "email": email,
+                "role": role,
+                "date_created": Decimal(datetime.datetime.utcnow().timestamp()),
+            }
+        )
+        status_code = response['ResponseMetadata']['HTTPStatusCode']
+        assert status_code == 200
+
+    @staticmethod
+    def get_invites(email):
+        try:
+            response = registry_db.query(
+                KeyConditionExpression=Key('partition_key').eq('invite:%s' % email)
+            )
+
+            invited_registeries = []
+            for invite in response['Items']:
+                invited_registeries.append({
+                    'registry_id': invite['sort_key'],
+                    'role': invite['role'],
+                    'email': invite['email'],
+                })
+
+            return invited_registeries
+        except ClientError as e:
+            print(e)
 
-class FlagTypes(str, Enum):    
+
+class FlagTypes(str, Enum):
     needs_discussion = 'Needs Discussion'
     review_with_psychiatrist = 'Review with Psychiatrist'
     safety_risk = 'Safety Risk'
 
 
 class ContactTypes(str, Enum):
     initial_assessment = 'Initial Assessment'
@@ -27,43 +129,37 @@
 
 class TreatmentLogScore(BaseModel):
     score_name: str
     score_value: int
 
 
 class TreatmentLog(BaseModel):
-    patient_mrn: Optional[str] = None  # TODO: We should remove this field since it's already in PatientRegistry
+    id: str = None
+    patient_mrn: Optional[str] = None
     provider: Optional[str] = None
-    
     no_show: Optional[bool] = False
-
     flag: Optional[FlagTypes] = None
+    cp_npi: Optional[str] = None
+    problems_list: Optional[str] = None
     weeks_in_treatment: int
     contact_type: ContactTypes
     visit_type: VisitTypes
-
     scores: List[TreatmentLogScore] = []
-
     minutes: Optional[float] = None
-
-    # TODO: Need to implement a notification workflow
     sms_reminder_sent_date: Optional[float] = None
     sms_conformation_received_date: Optional[float] = None
     total_sms_reminders_sent: Optional[int] = 0
-
-    # TODO: Need to implement a notification workflow
     email_reminder_sent_date: Optional[float] = None
     email_conformation_received_date: Optional[float] = None
     total_email_reminders_sent: Optional[int] = 0
+    date: float
 
-    # TODO: Allow the ability to schedule future sessions
-    date: float #TODO: Refactor this to created_date     
 
 class EventLog(BaseModel):
-    id: str    
+    id: str
     system: Optional[str] = None
     data: Optional[dict] = None
     created_date: float
     modified_date: float
 
 
 class AuditLog(BaseModel):
@@ -84,88 +180,16 @@
 class PatientStatysTypes(str, Enum):
     enrolled = 'Enrolled'
     treatment = 'Treatment'
     relapse_prevention_plan = 'Relapse Prevention Plan'
     deactivated = 'Deactivated'
 
 
-class RegistryIntegration(BaseModel):
-    name: str
-    api_key: str
-
-
-class RegistryModel(RegistryDBBaseModel):
+class AkelloApp(BaseModel):
     id: str
+    group: str
+    status: str
     name: str
     description: str
-    modified_date: float
-    created_date: float
-    members: int = 0
-    active_patients: int = 0
-    questionnaires: List[dict] = None
-    integrations: List[RegistryIntegration] = []
-    logo_url: Optional[str] = None
-
-    @property
-    def object_type(self) -> str:
-        return 'registry'
-
-    @property
-    def sort_key(self) -> str:
-        return 'metadata'
-
-
-class PatientRegistry(RegistryDBBaseModel):
-    id: Optional[str] = None
-    patient_flag: Optional[FlagTypes] = None
-    patient_mrn: str
-    date_created: float = datetime.datetime.utcnow().timestamp()
-    date_graduated: Optional[float] = None
-    date_modified: float = datetime.datetime.utcnow().timestamp()
-
-    payer: Optional[str] = None
-
-    first_name: str
-    last_name: str
-    phone_number: str
-    email: str
-    date_of_birth: str
-    treatment_logs: List[TreatmentLog] = []
-    event_logs: List[EventLog] = []
-    audit_logs: List[AuditLog] = []
-    flags: List[dict] = []
-
-    status: PatientStatysTypes = PatientStatysTypes.enrolled
-
-    initial_assessment: Optional[int] = None
-    last_follow_up: Optional[int] = None
-    last_psychiatric_consult: Optional[int] = None
-
-    relapse_prevention_plan: Optional[int] = None
-    total_sessions: Optional[int] = 0
-    weeks_since_initial_assessment: Optional[int] = 0  # TODO: This gets calculated from the client side, remove field
-    minutes_this_month: Optional[int] = 0  # TODO: This gets calculated from the client side, remove field
-    schema_version: Optional[str] = None
-
-    def toJson(self):
-        data = json.loads(self.model_dump_json())
-        data['partition_key'] = self.partition_key
-        data['sort_key'] = self.sort_key
-        return data
-
-    @property
-    def object_type(self):
-        return 'registry-patient'
-
-    @property
-    def sort_key(self) -> str:
-        return self.patient_mrn
-
-    model_config = {
-        "json_schema_extra": {
-            "examples": [
-                {
-                    "name": "Foo",
-                }
-            ]
-        }
-    }
+    logo: str
+    react_component: str
+    configs: dict
```

### Comparing `akello-0.0.19/akello/fhir/hl7/README.md` & `akello-0.0.20/akello/fhir/hl7/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/fhir/hl7/fhir_v6_models.py` & `akello-0.0.20/akello/fhir/hl7/fhir_v6_models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/screeners/R4/gad7.R4.json` & `akello-0.0.20/akello/screeners/R4/gad7.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/screeners/R4/phq9.R4.json` & `akello-0.0.20/akello/screeners/R4/phq9.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/screeners/questionnaires/gad7.json` & `akello-0.0.20/akello/screeners/questionnaires/gad7.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/screeners/questionnaires/phq9.json` & `akello-0.0.20/akello/screeners/questionnaires/phq9.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/akello/services/registry.py` & `akello-0.0.20/akello/services/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import os, datetime, random, uuid, json
+import datetime, random, uuid, json
 from decimal import Decimal
-from akello.dynamodb.models.registry import RegistryModel, TreatmentLog, PatientRegistry
-from akello.dynamodb import registry_db
+from akello.db.models import RegistryModel, TreatmentLog, PatientRegistry
+from akello.db.types import ContactTypes
+from akello.db.connector.dynamodb import registry_db
 from akello.services import BaseService
+from akello.services.stripe_payment import StripePaymentService
 from boto3.dynamodb.conditions import Key
 from botocore.exceptions import ClientError
 
 
-
 class RegistryService(BaseService):
 
     # TODO: We need decorator for permissions
     # TODO: We need to add logging
     # TODO: required roles: ['create registry']
     # the user object should be a validated one. Meaning there is no way its directly
     # from a web request where a user can set their roles
@@ -50,33 +51,44 @@
 
         try:
             response = registry_db.get_item(
                 Key={
                     'partition_key': 'registry:%s' % registry_id,
                     'sort_key': 'metadata'
                 }
-            )
-            print(response)
+            )            
         except ClientError as e:
             print(e)
-            print(e.response['No item found'])
+            print(e.response['No item found'])        
 
         status_code = response['ResponseMetadata']['HTTPStatusCode']
         assert status_code == 200
+        
+        return response['Item']                
 
-        return response['Item']
+
+    @staticmethod
+    def set_stripe_customer_id(registry_id, stripe_customer_id):
+        RegistryModel.set_attribute('registry:%s' % registry_id, 'metadata', 'stripe_customer_id', stripe_customer_id)
+
+    @staticmethod
+    def update_registry_akello_apps(registry_id, akello_apps):
+        RegistryModel.set_attribute('registry:%s' % registry_id, 'metadata', 'akello_apps', akello_apps)
+
+    @staticmethod
+    def set_measurements(registry_id, measurements):
+        RegistryModel.set_attribute('registry:%s' % registry_id, 'metadata', 'questionnaires', measurements)
 
     @staticmethod
     def update_stats(registry_id):
         patients = RegistryService.get_patients(registry_id)
         members = RegistryService.get_members(registry_id)
         RegistryModel.set_attribute('registry:%s' % registry_id, 'metadata', 'members', len(members))
         RegistryModel.set_attribute('registry:%s' % registry_id, 'metadata', 'active_patients', len(patients))
 
-
     @staticmethod
     def get_patient(registry_id, patient_id):
         try:
             response = registry_db.get_item(
                 Key={
                     'partition_key': 'registry-patient:%s' % registry_id,
                     'sort_key': patient_id
@@ -87,15 +99,15 @@
             print(e.response['No item found'])
 
         status_code = response['ResponseMetadata']['HTTPStatusCode']
         assert status_code == 200
 
         if 'Item' not in response:
             return None
-        
+
         return response['Item']
 
     @staticmethod
     def get_patients(registry_id, flag=None):
         try:
             response = registry_db.query(
                 KeyConditionExpression=Key('partition_key').eq('registry-patient:%s' % registry_id))
@@ -109,70 +121,84 @@
     def refer_patient(patient_registry: PatientRegistry):
         item = patient_registry.toJson()
 
         item = json.loads(json.dumps(item), parse_float=Decimal)
         item['partition_key'] = patient_registry.partition_key
         item['sort_key'] = patient_registry.sort_key
         response = registry_db.put_item(
-            Item=item
+            Item=item,
+            ConditionExpression='attribute_not_exists(partition_key) AND attribute_not_exists(sort_key)'
         )
         status_code = response['ResponseMetadata']['HTTPStatusCode']
         assert status_code == 200
 
     @staticmethod
     def update_patient(patient_registry: PatientRegistry):
         item = patient_registry.toJson()
-
         item = json.loads(json.dumps(item), parse_float=Decimal)
         item['partition_key'] = patient_registry.partition_key
         item['sort_key'] = patient_registry.sort_key
         response = registry_db.put_item(
             Item=item
         )
         status_code = response['ResponseMetadata']['HTTPStatusCode']
         assert status_code == 200
 
-
     @staticmethod
     def add_treatment_log(registry_id, sort_key, treatment_log: TreatmentLog):
-
-        UpdateExpression = "SET #att_name = list_append(#att_name, :treatment_logs), " \
-                           "flag = :flag," \
-                           "no_show = :no_show," \
-                           "initial_assessment = :initial_assessment, " \
-                           "last_follow_up = :last_follow_up, " \
-                           "last_psychiatric_consult = :last_psychiatric_consult, " \
-                           "relapse_prevention_plan = :relapse_prevention_plan, " \
-                           "weeks_since_initial_assessment = :weeks_since_initial_assessment "
-
-        ExpressionAttributeValues = {
+        """
+        Updates the treatment logs for a patient in the registry by appending a new treatment log entry.
+        It also updates specific attributes based on the contact type of the treatment log.
+
+        Args:
+            registry_id: The unique identifier for the registry.
+            sort_key: The sort key used for the database entry.
+            treatment_log: An instance of TreatmentLog representing the new treatment log to be added.
+        """
+        # Define the base update expression and attribute values
+        update_expression = ("SET #treatment_logs = list_append(#treatment_logs, :treatment_logs), "
+                             "flag = :flag, no_show = :no_show, "
+                             "weeks_since_initial_assessment = :weeks_since_initial_assessment")
+        expression_attribute_values = {
             ':treatment_logs': [json.loads(treatment_log.model_dump_json(), parse_float=Decimal)],
             ':flag': treatment_log.flag,
             ':no_show': treatment_log.no_show,
-            ':initial_assessment': Decimal(treatment_log.date),
-            ':last_follow_up': Decimal(treatment_log.date),
-            ":last_psychiatric_consult": Decimal(treatment_log.date),
-            ":relapse_prevention_plan": Decimal(treatment_log.date),
             ":weeks_since_initial_assessment": 0
         }
 
+        # Conditional updates for specific contact types
+        contact_type_updates = {
+            ContactTypes.follow_up: "last_follow_up",
+            ContactTypes.initial_assessment: "initial_assessment",
+            ContactTypes.psychiatric_consultation: "last_psychiatric_consult",
+            ContactTypes.relapse_prevention: "relapse_prevention_plan",
+        }
+
+        if treatment_log.contact_type in contact_type_updates:
+            field_name = contact_type_updates[treatment_log.contact_type]
+            update_expression += f", {field_name} = :{field_name}"
+            expression_attribute_values[f":{field_name}"] = Decimal(treatment_log.date)
+
+        # Execute the update operation
         response = registry_db.update_item(
             Key={
-                'partition_key': 'registry-patient:%s' % registry_id,
+                'partition_key': f'registry-patient:{registry_id}',
                 'sort_key': sort_key
             },
-            UpdateExpression=UpdateExpression,
+            UpdateExpression=update_expression,
             ExpressionAttributeNames={
-                "#att_name": "treatment_logs",
+                "#treatment_logs": "treatment_logs",
             },
-            ExpressionAttributeValues=ExpressionAttributeValues,
+            ExpressionAttributeValues=expression_attribute_values,
             ReturnValues="UPDATED_NEW"
         )
+
+        # Check the response status code
         status_code = response['ResponseMetadata']['HTTPStatusCode']
-        assert status_code == 200
+        assert status_code == 200, "Failed to update the treatment log."
 
 
     @staticmethod
     def get_members(registry_id):
         try:
             response = registry_db.query(
                 KeyConditionExpression=Key('partition_key').eq('registry-user:%s' % registry_id)
```

### Comparing `akello-0.0.19/akello/services/tests/__init__.py` & `akello-0.0.20/akello/services/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/.gitignore` & `akello-0.0.20/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 .pypirc
 
+.storage/
+
+synthetic_data/fhir*
+
 venv/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `akello-0.0.19/LICENSE` & `akello-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `akello-0.0.19/pyproject.toml` & `akello-0.0.20/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "akello"
-version = "0.0.19"
+version = "0.0.20"
 authors = [
   { name="Vijay Selvaraj", email="vijay@akellohealth.com" },
 ]
 description = "FastAPI server akello.io"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     "Programming Language :: Python :: 3",
 ]
+
 dependencies = [
     'fastapi',
     'boto3',
     'pydantic',
     'pydantic-settings',
     'fastapi_cognito',
     'uvicorn',
     'requests',
     'mangum',
     'aws_lambda_powertools',
+    'stripe',
+    'sendgrid',
+    'aiofiles',
+    'python-multipart',
+    'flatten_json',
+    'jsonschema'
 ]
 
 [project.urls]
 Homepage = "https://akello.io"
 Issues = "https://github.com/akello-io/akello/issues"
```

