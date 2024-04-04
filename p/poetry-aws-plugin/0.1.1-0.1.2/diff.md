# Comparing `tmp/poetry_aws_plugin-0.1.1.tar.gz` & `tmp/poetry_aws_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.1.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.2.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.1.tar` & `poetry_aws_plugin-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-03-28 22:37:24.836848 poetry_aws_plugin-0.1.1/LICENSE
--rw-r--r--   0        0        0     2361 2024-03-29 00:52:51.944613 poetry_aws_plugin-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-28 22:37:24.837975 poetry_aws_plugin-0.1.1/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     6084 2024-03-29 00:47:13.824504 poetry_aws_plugin-0.1.1/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      683 2024-03-29 00:53:00.024118 poetry_aws_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-04 16:43:29.996219 poetry_aws_plugin-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2629 2024-04-04 16:49:21.086127 poetry_aws_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 16:43:29.996219 poetry_aws_plugin-0.1.2/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     6411 2024-04-04 16:52:36.096094 poetry_aws_plugin-0.1.2/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-04 16:49:47.766122 poetry_aws_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.2/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.1/LICENSE` & `poetry_aws_plugin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.1/README.md` & `poetry_aws_plugin-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Poetry AWS Plugin
 
 This is a poetry plugin to help with AWS CodeArtifact authorization by automatically getting the authorization token.
 
+When installing or publishing packages through poetry and running into a CodeArtifact-related authorization error, the plugin will automatically get the authorization token and retry the command.
+
 The plugin will try two methods of authorization, in this order:
 
 1. Use AWS credentials to run `codeartifact.GetAuthorizationToken`.
 2. Use AWS credentials to run `sts.AssumeRole`, then use that role to run `codeartifact.GetAuthorizationToken`.
 
 ## Installation
 
@@ -49,8 +51,8 @@
 poetry install
 ```
 
 You can find more details in AWS's [CodeArtifact authentication and tokens documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/tokens-authentication.html) and [CodeArtifact IAM documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/security_iam_service-with-iam.html).
 
 # Misc
 
-You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token.
+You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token. This may be useful in CI/CD pipelines and reduce poetry configuration.
```

### Comparing `poetry_aws_plugin-0.1.1/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.2/poetry_aws_plugin/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from typing import Any
 
 import boto3
 import requests
 
 from botocore.exceptions import ClientError
-from cleo.io.io import IO
+from cleo.io.io import IO, Verbosity
 from poetry.exceptions import PoetryException
 from poetry.plugins import Plugin
 from poetry.poetry import Poetry
 from poetry.utils.authenticator import Authenticator
 from poetry.utils.password_manager import HTTPAuthCredential
 
 POETRY_AWS_PLUGIN_ROLE_ARN_VAR = "POETRY_AWS_PLUGIN_ROLE_ARN"
@@ -56,26 +56,30 @@
         try:
             token_response = boto3.client("codeartifact").get_authorization_token(
                 domain=domain,
                 domainOwner=domain_owner,
             )
             return token_response["authorizationToken"]
         except ClientError as err:
-            io.write_line(f"\nError getting CodeArtifact token using current credentials: {err}\n")
+            io.write_line(
+                f"\nError getting CodeArtifact token using current credentials: {err}\n",
+                verbosity=Verbosity.VERBOSE,
+            )
             return ""
         except Exception as err:
             io.write_line("Unexpected error while getting CodeArtifact authorization token")
             raise err
 
     def get_auth_token_with_iam_role(domain: str, domain_owner: str) -> str:
         role_arn = os.environ.get(POETRY_AWS_PLUGIN_ROLE_ARN_VAR)
         if not role_arn:
             io.write_line(
                 f"\nError getting CodeArtifact token using IAM role: "
-                f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found\n"
+                f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found\n",
+                verbosity=Verbosity.VERBOSE,
             )
             return ""
 
         try:
             assume_role_response = boto3.client("sts").assume_role(
                 RoleArn=role_arn,
                 RoleSessionName=POETRY_AWS_PLUGIN_SESSION_NAME,
@@ -89,29 +93,33 @@
 
             token_response = session.client("codeartifact").get_authorization_token(
                 domain=domain,
                 domainOwner=domain_owner,
             )
             return token_response["authorizationToken"]
         except ClientError as err:
-            io.write_line(f"\nError getting CodeArtifact token using IAM role '{role_arn}': {err}\n")
+            io.write_line(
+                f"\nError getting CodeArtifact token using IAM role '{role_arn}': {err}\n",
+                verbosity=Verbosity.VERBOSE,
+            )
             return ""
         except Exception as err:
             io.write_line(
                 "Unexpected error while assuming CodeArtifact role and getting CodeArtifact authorization token"
             )
             raise err
 
     def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
         return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
     def get_auth_token(domain: str, domain_owner: str) -> str:
         io.write_line(
             "\nGetting new CodeArtifact authorization token for "
-            f"domain '{domain}' and domain owner '{domain_owner}'\n"
+            f"domain '{domain}' and domain owner '{domain_owner}'\n",
+            verbosity=Verbosity.VERBOSE,
         )
 
         is_valid = validate_credentials()
         if not is_valid:
             return ""
 
         # We'll try these methods to get the CodeArtifact token
@@ -142,15 +150,18 @@
             match = re.match(CODEARTIFACT_URL_REGEX, response.url)
             domain, domain_owner = match.groups()
 
             auth_token = get_auth_token(domain, domain_owner)
             if not auth_token:
                 raise PoetryException(RETRY_ERROR_MESSAGE)
 
-            io.write_line("\nSuccessfully got CodeArtifact authorization token!\n\nRetrying request...\n")
+            io.write_line(
+                "\nSuccessfully got CodeArtifact authorization token!\n\nRetrying request...\n",
+                verbosity=Verbosity.VERBOSE,
+            )
 
             # Overwrite the credentials for this URL
             self._credentials[url] = HTTPAuthCredential(username="aws", password=auth_token)
 
             # Now retry the original request with new credentials
             return request(self, method=method, url=url, raise_for_status=raise_for_status, **kwargs)
```

### Comparing `poetry_aws_plugin-0.1.1/pyproject.toml` & `poetry_aws_plugin-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.1"
+version = "0.1.2"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
-repository = "https://github.com/xiasong/poetry-aws-plugin"
+repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 boto3 = "^1.34.71"
 poetry = "^1.7.0"
```

### Comparing `poetry_aws_plugin-0.1.1/PKG-INFO` & `poetry_aws_plugin-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
-Home-page: https://github.com/xiasong/poetry-aws-plugin
+Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.71,<2.0.0)
 Requires-Dist: poetry (>=1.7.0,<2.0.0)
-Project-URL: Repository, https://github.com/xiasong/poetry-aws-plugin
+Project-URL: Repository, https://github.com/xiasongh/poetry-aws-plugin
 Description-Content-Type: text/markdown
 
 # Poetry AWS Plugin
 
 This is a poetry plugin to help with AWS CodeArtifact authorization by automatically getting the authorization token.
 
+When installing or publishing packages through poetry and running into a CodeArtifact-related authorization error, the plugin will automatically get the authorization token and retry the command.
+
 The plugin will try two methods of authorization, in this order:
 
 1. Use AWS credentials to run `codeartifact.GetAuthorizationToken`.
 2. Use AWS credentials to run `sts.AssumeRole`, then use that role to run `codeartifact.GetAuthorizationToken`.
 
 ## Installation
 
@@ -69,9 +71,9 @@
 poetry install
 ```
 
 You can find more details in AWS's [CodeArtifact authentication and tokens documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/tokens-authentication.html) and [CodeArtifact IAM documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/security_iam_service-with-iam.html).
 
 # Misc
 
-You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token.
+You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token. This may be useful in CI/CD pipelines and reduce poetry configuration.
```

